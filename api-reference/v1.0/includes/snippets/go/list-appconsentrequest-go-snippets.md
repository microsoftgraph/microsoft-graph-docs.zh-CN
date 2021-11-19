---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ff59111cf7a51cdb33c14fec0c08ea7a03e0556
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103810"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.IdentityGovernance().AppConsent().AppConsentRequests().Get(options)


```