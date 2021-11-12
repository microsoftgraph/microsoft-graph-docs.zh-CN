---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22a98a4d67dc49e07eaf42e736062ff8f8cb3bb04943f48d40394b9066685791
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328708"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Fido2AuthenticationMethodCollectionPage fido2Methods = graphClient.me().authentication().fido2Methods()
    .buildRequest()
    .get();

```