---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1219f8cc4b23e159c199379b4d9575129cbb4ddf
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60983896"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

accessPackageId := "accessPackage-id"
graphClient.IdentityGovernance().EntitlementManagement().AccessPackagesById(&accessPackageId).Delete(options)


```