---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9ce614f28e16936c171147e98cf4b6db10713d1e54f81a95305eb62b32cb4f5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162502"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.compliance().ediscovery().cases("2192ca408ea2410eba3bec8ae873be6b").custodians("45454331323337443946343043464239")
    .activate()
    .buildRequest()
    .post();

```