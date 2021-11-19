---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f9b7f40973d88fa3e4c1e3a21b98a5cf2c1575d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098370"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

domainId := "domain-id"
graphClient.DomainsById(&domainId).Delete(options)


```