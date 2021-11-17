---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2b3d08803de0a44222552e873dd467399d978c61de0ca44cc2038d5a295d710
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105639"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CaseCollectionPage cases = graphClient.compliance().ediscovery().cases()
    .buildRequest()
    .get();

```