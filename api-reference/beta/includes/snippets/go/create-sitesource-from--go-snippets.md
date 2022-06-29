---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 132ea7e0be28f2394d18d59eaae55281d3e2af7f
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446701"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSiteSource()
site := msgraphsdk.NewSite()
requestBody.SetSite(site)
webUrl := "https://m365x809305.sharepoint.com/sites/Retail"
site.SetWebUrl(&webUrl)
ediscoveryCaseId := "ediscoveryCase-id"
ediscoveryHoldPolicyId := "ediscoveryHoldPolicy-id"
result, err := graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).LegalHoldsById(&ediscoveryHoldPolicyId).SiteSources().Post(requestBody)


```