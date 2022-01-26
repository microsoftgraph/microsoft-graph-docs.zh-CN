---
title: educationSynchronizationDataProvider 资源类型
description: '表示源 SIS 架构。 这允许系统了解如何将传入数据映射到Azure Active Directory (Azure AD) 架构。 '
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 869b24f5db8619caf3d60c17538f7ed4f8d932a5
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225754"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a>educationSynchronizationDataProvider 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示要用作 [educationSynchronizationProfile]的同步源的数据提供程序。

> [!NOTE]
> 此复杂类型为抽象类型。 请参阅列出的特定类型的数据提供程序。


**提供程序**

| Data Provider                                                             | 说明                                                                                        |
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------- |
| [educationCsvDataProvider]                                                | 上传到配置文件的 SAS URL 的 [CSV 文件](../api/educationsynchronizationprofile-uploadurl.md) |
| [educationOneRosterApiDataProvider](educationonerosterapidataprovider.md) | OneRoster v1.1 API                                                                                 |
| [educationPowerSchoolDataProvider]                                        | PowerSchool API                                                                                    |

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationDataProvider"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationSynchronizationDataProvider"
}
```


[educationsynchronizationprofile]: educationsynchronizationprofile.md
[educationcsvdataprovider]: educationCsvDataProvider.md
[educationsynchronizationdataprovider]: educationSynchronizationDataProvider.md
[educationpowerschooldataprovider]: educationPowerSchoolDataProvider.md
[educationcsvdataprovider]: educationCsvDataProvider.md
