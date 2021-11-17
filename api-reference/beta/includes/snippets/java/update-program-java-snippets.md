---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0c9f8d86b7edfa0adb4040f01ea6104aec3003cfaadb7f57e3e3ae0268a6c01
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902488"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Program program = new Program();
program.displayName = "testprogram3 new name";

graphClient.programs("7e59d237-2fb0-4e5d-b7bb-d4f9f9129213")
    .buildRequest()
    .patch(program);

```