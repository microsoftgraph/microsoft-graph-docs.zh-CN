---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9abb8916738ed53edf3f9ed04ee118384492308e
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61347000"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageCatalogId := "accessPackageCatalog-id"
graphClient.IdentityGovernance().EntitlementManagement().CatalogsById(&accessPackageCatalogId).Delete(nil)


```