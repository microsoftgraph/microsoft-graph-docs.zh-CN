---
title: appConfigurationSettingItem 资源类型
description: 包含应用配置设置项的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 900a16544b0166263b7d40c428c2c4cbaf5a0bb6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830420"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="a0821-103">appConfigurationSettingItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="a0821-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="a0821-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a0821-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0821-105">包含应用配置设置项的属性。</span><span class="sxs-lookup"><span data-stu-id="a0821-105">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="a0821-106">属性</span><span class="sxs-lookup"><span data-stu-id="a0821-106">Properties</span></span>
|<span data-ttu-id="a0821-107">属性</span><span class="sxs-lookup"><span data-stu-id="a0821-107">Property</span></span>|<span data-ttu-id="a0821-108">类型</span><span class="sxs-lookup"><span data-stu-id="a0821-108">Type</span></span>|<span data-ttu-id="a0821-109">说明</span><span class="sxs-lookup"><span data-stu-id="a0821-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0821-110">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="a0821-110">appConfigKey</span></span>|<span data-ttu-id="a0821-111">String</span><span class="sxs-lookup"><span data-stu-id="a0821-111">String</span></span>|<span data-ttu-id="a0821-112">应用配置密钥。</span><span class="sxs-lookup"><span data-stu-id="a0821-112">app configuration key.</span></span>|
|<span data-ttu-id="a0821-113">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="a0821-113">appConfigKeyType</span></span>|[<span data-ttu-id="a0821-114">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="a0821-114">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="a0821-115">应用配置密钥类型。</span><span class="sxs-lookup"><span data-stu-id="a0821-115">app configuration key type.</span></span> <span data-ttu-id="a0821-116">可取值为：`stringType`、`integerType`、`realType`、`booleanType`、`tokenType`。</span><span class="sxs-lookup"><span data-stu-id="a0821-116">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="a0821-117">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="a0821-117">appConfigKeyValue</span></span>|<span data-ttu-id="a0821-118">String</span><span class="sxs-lookup"><span data-stu-id="a0821-118">String</span></span>|<span data-ttu-id="a0821-119">应用配置密钥值。</span><span class="sxs-lookup"><span data-stu-id="a0821-119">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0821-120">关系</span><span class="sxs-lookup"><span data-stu-id="a0821-120">Relationships</span></span>
<span data-ttu-id="a0821-121">无</span><span class="sxs-lookup"><span data-stu-id="a0821-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a0821-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a0821-122">JSON Representation</span></span>
<span data-ttu-id="a0821-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0821-123">Here is a JSON representation of the resource.</span></span>
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



