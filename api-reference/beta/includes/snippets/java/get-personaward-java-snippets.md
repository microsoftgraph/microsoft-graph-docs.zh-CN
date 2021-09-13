---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14c1ec695821fe65c62ff3ada450fab54ef9fb048ca508ee306e2972013b15ea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161185"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonAward personAward = graphClient.me().profile().awards("{id}")
    .buildRequest()
    .get();

```