---
title: cloudPcDomainJoinConfiguration 资源类型
description: 表示预配的云电脑设备如何加入 Azure Active Directory。
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 3f35fb4a2aca6e7d0abd197e0c982038de3729ca
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64587635"
---
# <a name="cloudpcdomainjoinconfiguration-resource-type"></a>cloudPcDomainJoinConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示预配的云电脑设备如何加入 Azure Active Directory (Azure AD) 。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|onPremisesConnectionId|String|与虚拟网络 IT 管理员匹配的 Azure 网络连接 ID 希望预配策略在创建云电脑时使用。 此属性可用于两种域加入类型：已加入Azure AD _混合_ Azure AD _联接_。 如果输入 **onPremisesConnectionId**，将 **regionName 保留** 为空。|
|regionName|String|IT 管理员希望预配策略创建云电脑的受支持的 Azure 区域。 基础虚拟网络由 Windows 365 服务创建和管理。 只有在 IT 管理员选择加入域类型Azure AD才能输入。 如果输入 **regionName**，则 **onPremisesConnectionId 保留** 为空。|
|type|[cloudPcDomainJoinType](#cloudpcdomainjointype-values)|指定预配的云电脑如何加入 Azure AD。 如果选择类型，则 `hybridAzureADJoin` 仅提供 **onPremisesConnectionId** 属性的值，将 **regionName 保留** 为空。 如果选择类型， `azureADJoin` 请提供 **onPremisesConnectionId** 或 **regionName 的值**。 可能的值包括 `azureADJoin`、`hybridAzureADJoin`、`unknownFutureValue`。|

### <a name="cloudpcdomainjointype-values"></a>cloudPcDomainJoinType 值

|成员|说明|
|:---|:---|
|azureADJoin|仅联接到Azure AD。 可以分配仅云用户和混合用户并登录到云电脑。|
|hybridAzureADJoin|加入本地 AD 和 Azure AD。 只能分配混合用户并登录到云电脑。|
|unknownFutureValue|可发展枚举 sentinel 值。 请勿使用。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcDomainJoinConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcDomainJoinConfiguration",
  "type": "String",
  "regionName": "String",
  "onPremisesConnectionId": "String"
}
```
