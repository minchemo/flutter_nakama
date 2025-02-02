## 1.0.0-dev.2

* Full removed exported references of the underlaying raw datastructures
* Refactored realtime client

## 1.0.0-dev.1

* Changed License from MIT to Apache 2.0
* **Breaking:** Refactored the SDK to use own models instead of returning the underlaying Protobuf objects
* Most of the functionality added to achieve a stable release:
  * Authentication (Session refresh, missing drivers, linking and unlinking)
  * Leaderboard 
  * Friends & Groups
  * Notifications
  * Tournaments
  * Matches

## 0.1.6

* Full storage object support 🎉
* **Breaking** `readStorageObject()` returns now `Future<StorageObject?>` instead of `Future<StorageObject>`. Future resolves with `null` in case there was no element found with given key.
* Adds submitting and listing leaderboard records (more WIP)
* Adds `updateAccount()` method
* Bumps dependencies and API client to latest versions

## 0.1.5

* Adds [Real-Time chat](https://heroiclabs.com/docs/nakama/concepts/chat)
* Fixed missing session passing on `writeStorageObject()` (issue with multiple clients)

## 0.1.4
* Adds `onError()` and `onDone()` callbacks to `NakamaWebsocketClient`

## 0.1.3
* Fixes that the given server key was ignored

## 0.1.2
* Fully implements all authentication methods
* Enhanced documentation and adds link to package

## 0.1.1
* Fixed analyzer issues on web platform
* **Breaking Change:** use `getNakamaClient()` instead of `NakamaBaseClient.adaptive()`

## 0.1.0
* First release