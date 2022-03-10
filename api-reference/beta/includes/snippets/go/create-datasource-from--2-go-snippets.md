---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d4de347418ef703de9fdbaf5d1525886a54c1d2
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412590"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/custodians/ab3a628a383045eba344b3caecba3104/userSources/31423539-3846-4333-4136-353644383531",
}
options := &msgraphsdk.DataSourceRequestBuilderPostOptions{
    Body: requestBody,
}
caseId := "case-id"
sourceCollectionId := "sourceCollection-id"
dataSourceId := "dataSource-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).SourceCollectionsById(&sourceCollectionId).CustodianSourcesById(&dataSourceId).Post(options)


```