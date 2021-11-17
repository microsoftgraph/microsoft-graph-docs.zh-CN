---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7602ad09b52843baef8f3637d6bd9d1231d999b2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60996784"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.IdentityGovernance().TermsOfUse().Agreements().Get(options)


```