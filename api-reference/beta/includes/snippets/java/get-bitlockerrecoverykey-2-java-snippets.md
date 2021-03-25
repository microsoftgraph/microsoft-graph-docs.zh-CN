---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 604b74d25b12b490a100fa047c5cd2df71494d3d
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209057"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ocp-client-name", "\"My Friendly Client\""));
requestOptions.add(new HeaderOption("ocp-client-version", "\"1.2\""));

BitlockerRecoveryKeyCollectionPage recoveryKeys = graphClient.informationProtection().bitlocker().recoveryKeys()
    .buildRequest( requestOptions )
    .filter("deviceId eq '1ab40ab2-32a8-4b00-b6b5-ba724e407de9'")
    .get();

```