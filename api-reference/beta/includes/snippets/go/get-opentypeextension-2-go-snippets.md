---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ec9a4db669bf6a01e97176d66c36a414320dd84
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288959"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
eventId := "event-id"
extensionId := "extension-id"
result, err := graphClient.GroupsById(&groupId).EventsById(&eventId).ExtensionsById(&extensionId).Get(nil)


```