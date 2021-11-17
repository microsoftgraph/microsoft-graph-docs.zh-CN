---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da78175ad1b7d6f3dff60b021877922fdf5fd81b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60984456"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

outlookCategoryId := "outlookCategory-id"
result, err := graphClient.Me().Outlook().MasterCategoriesById(&outlookCategoryId).Get(options)


```