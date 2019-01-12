---
title: appConfigurationSettingItem 资源类型
description: 包含应用配置设置项的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ddb7b503ff14e6499342fafc2d0cf5ab8e670138
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960334"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="b9234-103">appConfigurationSettingItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="b9234-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="b9234-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b9234-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9234-105">包含应用配置设置项的属性。</span><span class="sxs-lookup"><span data-stu-id="b9234-105">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="b9234-106">属性</span><span class="sxs-lookup"><span data-stu-id="b9234-106">Properties</span></span>
|<span data-ttu-id="b9234-107">属性</span><span class="sxs-lookup"><span data-stu-id="b9234-107">Property</span></span>|<span data-ttu-id="b9234-108">类型</span><span class="sxs-lookup"><span data-stu-id="b9234-108">Type</span></span>|<span data-ttu-id="b9234-109">说明</span><span class="sxs-lookup"><span data-stu-id="b9234-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9234-110">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="b9234-110">appConfigKey</span></span>|<span data-ttu-id="b9234-111">String</span><span class="sxs-lookup"><span data-stu-id="b9234-111">String</span></span>|<span data-ttu-id="b9234-112">应用配置密钥。</span><span class="sxs-lookup"><span data-stu-id="b9234-112">app configuration key.</span></span>|
|<span data-ttu-id="b9234-113">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="b9234-113">appConfigKeyType</span></span>|[<span data-ttu-id="b9234-114">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="b9234-114">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="b9234-115">应用配置密钥类型。</span><span class="sxs-lookup"><span data-stu-id="b9234-115">app configuration key type.</span></span> <span data-ttu-id="b9234-116">可取值为：`stringType`、`integerType`、`realType`、`booleanType`、`tokenType`。</span><span class="sxs-lookup"><span data-stu-id="b9234-116">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="b9234-117">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="b9234-117">appConfigKeyValue</span></span>|<span data-ttu-id="b9234-118">String</span><span class="sxs-lookup"><span data-stu-id="b9234-118">String</span></span>|<span data-ttu-id="b9234-119">应用配置密钥值。</span><span class="sxs-lookup"><span data-stu-id="b9234-119">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9234-120">关系</span><span class="sxs-lookup"><span data-stu-id="b9234-120">Relationships</span></span>
<span data-ttu-id="b9234-121">无</span><span class="sxs-lookup"><span data-stu-id="b9234-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b9234-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b9234-122">JSON Representation</span></span>
<span data-ttu-id="b9234-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9234-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConfigurationSettingItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConfigurationSettingItem",
  "appConfigKey": "String",
  "appConfigKeyType": "String",
  "appConfigKeyValue": "String"
}
```



