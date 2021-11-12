---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97234d654a8b380281dea994ebe2b3e4b150dca7c93fbfbff3b7ad89556b5201
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329003"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintService printService = graphClient.print().services("{id}")
    .buildRequest()
    .get();

```