---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6787395a887310a7071c25d654fb3e407133d0b
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210305"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectorySettingCollectionPage settings = graphClient.settings()
    .buildRequest()
    .get();

```