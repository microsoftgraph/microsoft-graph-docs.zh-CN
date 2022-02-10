---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 007326b834f602a2c7a0033782ba5bfe51d9b0d6
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519613"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackageCatalog()
displayName := "Catalog One"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.AccessPackageCatalogRequestBuilderPatchOptions{
    Body: requestBody,
}
accessPackageCatalogId := "accessPackageCatalog-id"
graphClient.IdentityGovernance().EntitlementManagement().CatalogsById(&accessPackageCatalogId).Patch(options)


```