---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe05ec6eb530a9e52f1ef2e91a08344078dc8f2e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61016636"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Me().ScopedRoleMemberOf().Get(options)


```