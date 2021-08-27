---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d375842e043d7101672c396f510cfb2cd7751c240cb7c97ed1bb389ebefd1c0d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409663"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserCollectionPage users = graphClient.users()
    .buildRequest()
    .get();

```