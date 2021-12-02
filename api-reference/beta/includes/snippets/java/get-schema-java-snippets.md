---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ff8ed0bd210ff5a87951b0bfe8381c7056d71b5c04afdbdfb999a4ecade90ce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219757"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Schema schema = graphClient.external().connections("contosohr").schema()
    .buildRequest()
    .get();

```