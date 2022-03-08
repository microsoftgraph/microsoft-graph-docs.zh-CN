---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d4db01a3d96805207db3fc63eedd0a818fbd4bd
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338357"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageCatalogId := "accessPackageCatalog-id"
customAccessPackageWorkflowExtensionId := "customAccessPackageWorkflowExtension-id"
graphClient.IdentityGovernance().EntitlementManagement().AccessPackageCatalogsById(&accessPackageCatalogId).CustomAccessPackageWorkflowExtensionsById(&customAccessPackageWorkflowExtensionId).Delete(nil)


```