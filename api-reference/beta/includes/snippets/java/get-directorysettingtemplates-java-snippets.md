---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b1d1ed7b670b57537ef36c67ccd5c73ebf2b6fb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978443"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectorySettingTemplateCollectionPage directorySettingTemplates = graphClient.directorySettingTemplates()
    .buildRequest()
    .get();

```