---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6011353466d951cfd1580d1624c54e8bd36a1d90
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61007329"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.RoleManagement().Directory().RoleDefinitions().Get(options)


```