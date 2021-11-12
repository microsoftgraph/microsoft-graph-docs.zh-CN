---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23a69930af78d9ea93532950148565bdf04b56ed731852ac2579b6a0630b983b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219015"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MessageCollectionPage messages = graphClient.me().mailFolders("AAMkAGVmMDEzM").messages()
    .buildRequest()
    .get();

```