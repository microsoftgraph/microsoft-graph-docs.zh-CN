---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f23a7f9503eb74a1845d0a609fdd0f199c7ccae190900cd5f197c443626ec03f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219869"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserSource userSource = graphClient.compliance().ediscovery().cases("4c8f8f70-7785-4bd4-b296-c98376a2c5e1").custodians("2192ca408ea2410eba3bec8ae873be6b").userSources("46384443-4137-3032-3437-363939433735")
    .buildRequest()
    .get();

```