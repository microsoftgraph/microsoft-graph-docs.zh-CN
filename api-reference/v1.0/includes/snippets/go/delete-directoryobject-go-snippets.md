---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6d67a5dafcf5c6462880dde0d12a1b134d88662
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60974010"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

directoryObjectId := "directoryObject-id"
graphClient.DirectoryObjectsById(&directoryObjectId).Delete(options)


```