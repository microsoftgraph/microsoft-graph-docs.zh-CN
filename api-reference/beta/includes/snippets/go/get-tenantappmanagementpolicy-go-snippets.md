---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec9f4f680ae9edfbe9bde045f20b637a128ef13e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092392"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Policies().DefaultAppManagementPolicy().Get(options)


```