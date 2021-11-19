---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e740d7a20d599a6fc51a3c534cf84c3a03957be5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099717"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

directoryObjectId := "directoryObject-id"
graphClient.DirectoryObjectsById(&directoryObjectId).Delete(options)


```