---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0ee2083e85c581d68792434db1372e0b56a1464
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61024595"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

educationUserId := "educationUser-id"
graphClient.Education().UsersById(&educationUserId).Patch(options)


```