---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b7c3847c101bb7382270069c0fe0b5d4ac76cb3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328510"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageCatalogId := "accessPackageCatalog-id"
customAccessPackageWorkflowExtensionId := "customAccessPackageWorkflowExtension-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageCatalogsById(&accessPackageCatalogId).CustomAccessPackageWorkflowExtensionsById(&customAccessPackageWorkflowExtensionId).Get()


```