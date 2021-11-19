---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04869fb30028361e5685add107e0c5341e61333e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093193"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

organizationId := "organization-id"
profileCardPropertyId := "profileCardProperty-id"
result, err := graphClient.OrganizationById(&organizationId).Settings().ProfileCardPropertiesById(&profileCardPropertyId).Get(options)


```