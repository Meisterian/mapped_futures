# Mapped Futures

This library contains the MappedFutures struct, which allows keys to be mapped to futures. Once added, the futures can be mutated or removed if you have the key. MappedFutures is implemented by adding a HashMap to FuturesUnordered, so futures will only be polled after being woken, and will complete out of order.
