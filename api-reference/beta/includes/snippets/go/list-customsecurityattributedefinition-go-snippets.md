---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d577c47794fd8ac9d56a3004297522606bb53d13
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224591"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Directory().CustomSecurityAttributeDefinitions().Get(options)


```