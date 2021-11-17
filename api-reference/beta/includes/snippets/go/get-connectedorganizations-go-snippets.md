---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5b03bf6ed198d14c0d05436ec163e87b4dc5c46
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61005647"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.IdentityGovernance().EntitlementManagement().ConnectedOrganizations().Get(options)


```