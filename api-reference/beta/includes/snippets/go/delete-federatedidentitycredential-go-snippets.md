---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a16278201660051f939baa5f95d3826e88f2771b
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412255"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

applicationId := "application-id"
federatedIdentityCredentialId := "federatedIdentityCredential-id"
result, err := graphClient.ApplicationsById(&applicationId).FederatedIdentityCredentialsById(&federatedIdentityCredentialId).Delete(nil)


```