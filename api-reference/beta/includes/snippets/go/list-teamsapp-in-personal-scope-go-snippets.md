---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a23e64e1929c76a1d9a30e9d633177241bc4757c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085670"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.TeamsAppsRequestBuilderGetQueryParameters{
    Expand: "appDefinitions($select=id,displayName,allowedInstallationScopes)",
    Filter: "appDefinitions/any(a:a/allowedInstallationScopes%20has%20'personal')",
}
options := &msgraphsdk.TeamsAppsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.AppCatalogs().TeamsApps().Get(options)


```