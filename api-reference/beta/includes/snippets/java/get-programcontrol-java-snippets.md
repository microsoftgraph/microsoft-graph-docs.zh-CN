---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c65c7284f4ace7aa579a5e66d6d5c4dca253c14375b0eef61e0faaa02b8a182
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333326"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProgramControlCollectionPage programControls = graphClient.programControls()
    .buildRequest()
    .get();

```