---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16c921cad8bc03a870d24e0f9deeaaa299a8d511
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033425"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userId := "user-id"
result, err := graphClient.UsersById(&userId).Manager().Get(options)


```