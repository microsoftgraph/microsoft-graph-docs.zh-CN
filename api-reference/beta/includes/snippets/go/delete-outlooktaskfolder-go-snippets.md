---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a205e8c3ec70f43329b9cf2b24852ea43cea139
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61011513"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

outlookTaskFolderId := "outlookTaskFolder-id"
graphClient.Me().Outlook().TaskFoldersById(&outlookTaskFolderId).Delete(options)


```