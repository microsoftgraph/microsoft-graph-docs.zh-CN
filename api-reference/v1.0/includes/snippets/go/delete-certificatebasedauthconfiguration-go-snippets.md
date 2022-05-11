---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25fa2ed8558215779c79ce6cc54fe7f58bafc1ab
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329056"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

organizationId := "organization-id"
certificateBasedAuthConfigurationId := "certificateBasedAuthConfiguration-id"
graphClient.OrganizationById(&organizationId).CertificateBasedAuthConfigurationById(&certificateBasedAuthConfigurationId).Delete()


```