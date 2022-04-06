---
title: microsoftApplicationDataAccessSettings 资源类型
description: 表示用于确定从 Microsoft 应用访问Microsoft 365属于组织中用户的数据的设置。 例如，如果授权正确，那么只有 Microsoft 365 应用 (（如 Word 和 Excel) ）可以访问用户的 Microsoft 365 数据，或者其他 Microsoft 应用 (如 Windows) 是否可以访问该数据。
author: ttomi
ms.localizationpriority: medium
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 049089e4c3246beed9f459831cd7903dea9e4ce3
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589619"
---
# <a name="microsoftapplicationdataaccesssettings-resource-type"></a>microsoftApplicationDataAccessSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 _一_ 些设置，这些设置指定从 Microsoft 应用程序访问Microsoft 365属于组织中用户的数据。 例如，如果授权正确，那么只有 Microsoft 365 应用 (（如 Word 和 Excel) ）可以访问用户的 Microsoft 365 数据，或者其他 Microsoft 应用 (如 Windows) 是否可以访问该数据。

组织中 Microsoft 365 数据的示例包括 Word、Excel 和 PowerPoint 文档、Outlook 消息和 Teams 会议录制，Microsoft 应用中的用户已正确授权访问这些录制。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 microsoftApplicationDataAccessSettings](../api/organizationsettings-list-microsoftapplicationdataaccess.md)|[microsoftApplicationDataAccessSettings](microsoftapplicationdataaccesssettings.md)|获取 [microsoftApplicationDataAccessSettings](microsoftapplicationdataaccesssettings.md) 对象中的设置，该对象指定从 Microsoft 应用程序访问以Microsoft 365组织的用户数据。|
|[更新 microsoftApplicationDataAccessSettings](../api/microsoftapplicationdataaccesssettings-update.md)|[microsoftApplicationDataAccessSettings](microsoftapplicationdataaccesssettings.md)|更新 [microsoftApplicationDataAccessSettings](microsoftapplicationdataaccesssettings.md) 对象中的设置，该对象指定从 Microsoft 应用程序访问以Microsoft 365组织的用户数据。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|isEnabledForAllMicrosoftApplications|Boolean|`true`设置为 时，组织中所有用户都可以在 Microsoft 应用中访问Microsoft 365已授权访问的任何数据。 Microsoft 应用可以是一个Microsoft 365应用 (例如，Excel、Outlook) 或非Microsoft 365应用 (例如，Edge) 。 默认值为 `true`。 <br> 通过指定 **disabledForGroup** 属性中的组，可以禁用安全Azure AD部分用户的此访问权限。 <br> 设置为 时`false`，所有用户只能在 Microsoft 365应用中访问授权Microsoft 365数据。|
|disabledForGroup|String|允许成员Azure Active Directory (Azure AD) 安全组的 ID，该安全组Microsoft 365使用 Microsoft 365 应用访问数据，而不允许使用其他 Microsoft 应用（如 Edge）。 <br> This is only applicable if **isEnabledForAllMicrosoftApplications is** set to `true`.|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.microsoftApplicationDataAccessSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftApplicationDataAccessSettings",
  "isEnabledForAllMicrosoftApplications": "Boolean",
  "disabledForGroup": "String"
}
```
