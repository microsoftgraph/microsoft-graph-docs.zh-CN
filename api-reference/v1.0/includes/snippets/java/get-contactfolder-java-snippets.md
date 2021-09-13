---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 788bfea4dd4f89b53d298c3a84572cd7d2690afba1aaea5dc21731c75a28e2f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164040"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContactFolder contactFolder = graphClient.me().contactFolders("{id}")
    .buildRequest()
    .get();

```