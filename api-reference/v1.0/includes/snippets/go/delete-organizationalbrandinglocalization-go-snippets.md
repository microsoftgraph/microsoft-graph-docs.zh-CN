---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29ed1f93c1709c4555f14ab2fe2d03e52ba0abd8
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328188"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

organizationId := "organization-id"
organizationalBrandingLocalizationId := "organizationalBrandingLocalization-id"
graphClient.OrganizationById(&organizationId).Branding().LocalizationsById(&organizationalBrandingLocalizationId).Delete()


```