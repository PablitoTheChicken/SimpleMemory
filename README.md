# SimpleMemory

This tool is made to make the process of using MemoryStoreService more easy and faster to use.

## MemoryStore

- <b>Constructor</b><br />
    - `SimpleMemory.newQueue(Name: string) ` <br />
    - `SimpleMemory.newStortedMap(Name: string) ` <br />

- <b>Methods</b><br />
    - <b>Queue</b>
        - `Queue:Write(value: any, expiration: number, priority: number)`
        - `Queue:Read(count: number, allOrNothing: boolean, waitTimeout: number)`
        - `Queue:Remove(value: any, expiration: number, priority: number)`
    - <b>SortedMap</b>
        - `SortedMap:Set(key: string, value: any, expiration: number)`
        - `SortedMap:GetRange(direction: SortDirection, count: IntValue, exclusiveLowerBound: string?, exclusiveUpperBound: string?)`
        - `SortedMap:Update(key: string, callback: function, expiration: IntValue)`
        - `SortedMap:Remove(key: string)`
