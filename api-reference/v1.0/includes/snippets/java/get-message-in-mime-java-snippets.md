---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66770b2a1b51463e59372324e1cb6af39685b6f7
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41558997"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Stream stream = graphClient.me().messages("4aade2547798441eab5188a7a2436bc1").content()
    .buildRequest()
    .get();

```