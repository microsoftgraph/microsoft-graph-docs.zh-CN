---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93bd01d09e6f9da11bd0afe46ab7fa63b08b7df5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983201"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.trustFramework().policies("B2C_1A_SocialAndLocalAccounts_Base")
    .buildRequest()
    .delete();

```