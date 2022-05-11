---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5b899c74c7645fb650b35a4cb0450b9fc4944b8
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326122"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

agreementId := "agreement-id"
result, err := graphClient.IdentityGovernance().TermsOfUse().AgreementsById(&agreementId).Get()


```