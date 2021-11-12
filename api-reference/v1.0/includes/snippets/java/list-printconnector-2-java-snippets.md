---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a426872d9108bc7d4b0cf2f3fa88c9d2c8a576b3d775da9cad01a764ce48c722
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409682"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintConnectorCollectionWithReferencesPage connectors = graphClient.print().printers("{printerId}").connectors()
    .buildRequest()
    .get();

```