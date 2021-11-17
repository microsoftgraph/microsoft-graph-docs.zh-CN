---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a8af6a03aed266ba228ac5c21966dc6c9f79229725f76ca32b082571a1c8a55
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221079"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemPhoneCollectionPage phones = graphClient.me().profile().phones()
    .buildRequest()
    .get();

```