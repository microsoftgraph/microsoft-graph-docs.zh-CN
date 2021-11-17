---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97a696e834c7acca3e51b8caf2fec381674a68f9440aa74da16872fc72a63d3a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106512"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Place place = graphClient.places("3162F1E1-C4C0-604B-51D8-91DA78989EB1")
    .buildRequest()
    .get();

```