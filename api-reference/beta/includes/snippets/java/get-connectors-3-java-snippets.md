---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b7c16ae5a23b635b5c64700333f2f7d45acd8c7
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209239"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintConnectorCollectionWithReferencesPage connectors = graphClient.print().printers("{id}").connectors()
    .buildRequest()
    .get();

```