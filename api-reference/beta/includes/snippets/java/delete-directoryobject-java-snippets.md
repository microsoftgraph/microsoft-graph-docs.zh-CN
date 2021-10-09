---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12f4a87f8f71fd8d7e22a7324420cb2ba4d88c3138bf24439e019a8f7cb37f7a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106555"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directoryObjects("ffab4dce-9b82-49a6-b7c7-1a143106598c")
    .buildRequest()
    .delete();

```