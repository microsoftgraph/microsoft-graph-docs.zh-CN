---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac1f0eb52ddf689cde026dd6cbade457f72b616a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61030000"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

outlookTaskGroupId := "outlookTaskGroup-id"
result, err := graphClient.Me().Outlook().TaskGroupsById(&outlookTaskGroupId).TaskFolders().Get(options)


```