---
title: appConfigurationSettingItem 资源类型
description: 包含应用配置设置项的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b7f5492c9b54c9414db6a8332e218a1d7f0a50b1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403761"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="352db-103">appConfigurationSettingItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="352db-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="352db-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="352db-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="352db-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="352db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="352db-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="352db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="352db-107">包含应用配置设置项的属性。</span><span class="sxs-lookup"><span data-stu-id="352db-107">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="352db-108">属性</span><span class="sxs-lookup"><span data-stu-id="352db-108">Properties</span></span>
|<span data-ttu-id="352db-109">属性</span><span class="sxs-lookup"><span data-stu-id="352db-109">Property</span></span>|<span data-ttu-id="352db-110">类型</span><span class="sxs-lookup"><span data-stu-id="352db-110">Type</span></span>|<span data-ttu-id="352db-111">说明</span><span class="sxs-lookup"><span data-stu-id="352db-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="352db-112">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="352db-112">appConfigKey</span></span>|<span data-ttu-id="352db-113">String</span><span class="sxs-lookup"><span data-stu-id="352db-113">String</span></span>|<span data-ttu-id="352db-114">应用配置密钥。</span><span class="sxs-lookup"><span data-stu-id="352db-114">app configuration key.</span></span>|
|<span data-ttu-id="352db-115">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="352db-115">appConfigKeyType</span></span>|[<span data-ttu-id="352db-116">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="352db-116">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="352db-117">应用配置密钥类型。</span><span class="sxs-lookup"><span data-stu-id="352db-117">app configuration key type.</span></span> <span data-ttu-id="352db-118">可取值为：`stringType`、`integerType`、`realType`、`booleanType`、`tokenType`。</span><span class="sxs-lookup"><span data-stu-id="352db-118">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="352db-119">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="352db-119">appConfigKeyValue</span></span>|<span data-ttu-id="352db-120">String</span><span class="sxs-lookup"><span data-stu-id="352db-120">String</span></span>|<span data-ttu-id="352db-121">应用配置密钥值。</span><span class="sxs-lookup"><span data-stu-id="352db-121">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="352db-122">关系</span><span class="sxs-lookup"><span data-stu-id="352db-122">Relationships</span></span>
<span data-ttu-id="352db-123">无</span><span class="sxs-lookup"><span data-stu-id="352db-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="352db-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="352db-124">JSON Representation</span></span>
<span data-ttu-id="352db-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="352db-125">Here is a JSON representation of the resource.</span></span>
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




