# DynamicReturnFeeTestHook
[Git Source](https://github.com/uniswap/v4-core/blob/b619b6718e31aa5b4fa0286520c455ceb950276d/src/test/DynamicReturnFeeTestHook.sol) - Generated with [forge doc](https://book.getfoundry.sh/reference/forge/forge-doc)

**Inherits:**
[BaseTestHooks](contracts/v4/reference/core/test/BaseTestHooks.md)


## State Variables
### fee

```solidity
uint24 internal fee;
```


### manager

```solidity
IPoolManager manager;
```


## Functions
### setManager


```solidity
function setManager(IPoolManager _manager) external;
```

### setFee


```solidity
function setFee(uint24 _fee) external;
```

### beforeSwap


```solidity
function beforeSwap(address, PoolKey calldata, IPoolManager.SwapParams calldata, bytes calldata)
    external
    view
    override
    returns (bytes4, BeforeSwapDelta, uint24);
```

### forcePoolFeeUpdate


```solidity
function forcePoolFeeUpdate(PoolKey calldata _key, uint24 _fee) external;
```
