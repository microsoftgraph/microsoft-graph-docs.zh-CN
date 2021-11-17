---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a8b7caaf16501a6ffdd54573ad10b535b70334d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023749"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

outlookTaskFolderId := "outlookTaskFolder-id"
result, err := graphClient.Me().Outlook().TaskFoldersById(&outlookTaskFolderId).Tasks().Get(options)


```