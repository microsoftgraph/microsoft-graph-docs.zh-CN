---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df5ff5168620b608ffa95b0b759bc1a4b2251c50
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327626"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Reports().CredentialUserRegistrationDetails().Get()


```