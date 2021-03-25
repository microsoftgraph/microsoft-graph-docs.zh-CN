---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9dc6271dcf74b562719c22d9d9dc0b6a98a881a
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209410"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintConnectorCollectionWithReferencesPage connectors = graphClient.print().printers("{printerId}").connectors()
    .buildRequest()
    .get();

```