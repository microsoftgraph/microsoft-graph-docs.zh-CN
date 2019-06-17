---
title: appConfigurationSettingItem 资源类型
description: 包含应用配置设置项的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f001a02a1e4e3ef2a15fe5e606687896775a6d26
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991259"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="d7cae-103">appConfigurationSettingItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="d7cae-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="d7cae-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d7cae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7cae-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d7cae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7cae-106">包含应用配置设置项的属性。</span><span class="sxs-lookup"><span data-stu-id="d7cae-106">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="d7cae-107">属性</span><span class="sxs-lookup"><span data-stu-id="d7cae-107">Properties</span></span>
|<span data-ttu-id="d7cae-108">属性</span><span class="sxs-lookup"><span data-stu-id="d7cae-108">Property</span></span>|<span data-ttu-id="d7cae-109">类型</span><span class="sxs-lookup"><span data-stu-id="d7cae-109">Type</span></span>|<span data-ttu-id="d7cae-110">说明</span><span class="sxs-lookup"><span data-stu-id="d7cae-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7cae-111">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="d7cae-111">appConfigKey</span></span>|<span data-ttu-id="d7cae-112">String</span><span class="sxs-lookup"><span data-stu-id="d7cae-112">String</span></span>|<span data-ttu-id="d7cae-113">应用配置密钥。</span><span class="sxs-lookup"><span data-stu-id="d7cae-113">app configuration key.</span></span>|
|<span data-ttu-id="d7cae-114">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="d7cae-114">appConfigKeyType</span></span>|[<span data-ttu-id="d7cae-115">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="d7cae-115">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="d7cae-116">应用配置密钥类型。</span><span class="sxs-lookup"><span data-stu-id="d7cae-116">app configuration key type.</span></span> <span data-ttu-id="d7cae-117">可取值为：`stringType`、`integerType`、`realType`、`booleanType`、`tokenType`。</span><span class="sxs-lookup"><span data-stu-id="d7cae-117">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="d7cae-118">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="d7cae-118">appConfigKeyValue</span></span>|<span data-ttu-id="d7cae-119">String</span><span class="sxs-lookup"><span data-stu-id="d7cae-119">String</span></span>|<span data-ttu-id="d7cae-120">应用配置密钥值。</span><span class="sxs-lookup"><span data-stu-id="d7cae-120">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7cae-121">关系</span><span class="sxs-lookup"><span data-stu-id="d7cae-121">Relationships</span></span>
<span data-ttu-id="d7cae-122">无</span><span class="sxs-lookup"><span data-stu-id="d7cae-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7cae-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d7cae-123">JSON Representation</span></span>
<span data-ttu-id="d7cae-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7cae-124">Here is a JSON representation of the resource.</span></span>
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





