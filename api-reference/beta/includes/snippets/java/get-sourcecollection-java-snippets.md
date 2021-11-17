---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ee1a56247b5808d465fe621118e96d4b775242e2778849afe9de26cc269b5f6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215892"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SourceCollection sourceCollection = graphClient.compliance().ediscovery().cases("47746044-fd0b-4a30-acfc-5272b691ba5b").sourceCollections("1a9b4145d8f84e39bc45a7f68c5c5119")
    .buildRequest()
    .expand("lastEstimateStatisticsOperation")
    .get();

```