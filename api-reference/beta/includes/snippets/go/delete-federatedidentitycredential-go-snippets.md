---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5826717972f915bb2821f4bc1283d61b8f78967e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097484"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

applicationId := "application-id"
federatedIdentityCredentialId := "federatedIdentityCredential-id"
graphClient.ApplicationsById(&applicationId).FederatedIdentityCredentialsById(&federatedIdentityCredentialId).Delete(options)


```