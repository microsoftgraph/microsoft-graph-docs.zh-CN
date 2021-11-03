---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36599f12a51ca72a6514c5ceb7c612cbb27525fd
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694377"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Schema schema = graphClient.external().connections("contosohr").schema()
    .buildRequest()
    .get();

```