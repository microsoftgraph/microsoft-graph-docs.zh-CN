---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84fd4f8b891de165ccb1ac5edf3e132400ff4a3b1465bcc6aedc2185f8abdf06
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104302"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintServiceCollectionPage services = graphClient.print().services()
    .buildRequest()
    .get();

```