---
title: appConfigurationSettingItem 资源类型
description: 包含应用配置设置项的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bdc552bc2dcaf04990999c9414d2723284a568f2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48045465"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="e6b93-103">appConfigurationSettingItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="e6b93-103">appConfigurationSettingItem resource type</span></span>

<span data-ttu-id="e6b93-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6b93-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e6b93-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e6b93-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6b93-106">包含应用配置设置项的属性。</span><span class="sxs-lookup"><span data-stu-id="e6b93-106">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="e6b93-107">属性</span><span class="sxs-lookup"><span data-stu-id="e6b93-107">Properties</span></span>
|<span data-ttu-id="e6b93-108">属性</span><span class="sxs-lookup"><span data-stu-id="e6b93-108">Property</span></span>|<span data-ttu-id="e6b93-109">类型</span><span class="sxs-lookup"><span data-stu-id="e6b93-109">Type</span></span>|<span data-ttu-id="e6b93-110">说明</span><span class="sxs-lookup"><span data-stu-id="e6b93-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6b93-111">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="e6b93-111">appConfigKey</span></span>|<span data-ttu-id="e6b93-112">String</span><span class="sxs-lookup"><span data-stu-id="e6b93-112">String</span></span>|<span data-ttu-id="e6b93-113">应用配置密钥。</span><span class="sxs-lookup"><span data-stu-id="e6b93-113">app configuration key.</span></span>|
|<span data-ttu-id="e6b93-114">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="e6b93-114">appConfigKeyType</span></span>|[<span data-ttu-id="e6b93-115">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="e6b93-115">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="e6b93-116">应用配置密钥类型。</span><span class="sxs-lookup"><span data-stu-id="e6b93-116">app configuration key type.</span></span> <span data-ttu-id="e6b93-117">可取值为：`stringType`、`integerType`、`realType`、`booleanType`、`tokenType`。</span><span class="sxs-lookup"><span data-stu-id="e6b93-117">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="e6b93-118">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="e6b93-118">appConfigKeyValue</span></span>|<span data-ttu-id="e6b93-119">String</span><span class="sxs-lookup"><span data-stu-id="e6b93-119">String</span></span>|<span data-ttu-id="e6b93-120">应用配置密钥值。</span><span class="sxs-lookup"><span data-stu-id="e6b93-120">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6b93-121">关系</span><span class="sxs-lookup"><span data-stu-id="e6b93-121">Relationships</span></span>
<span data-ttu-id="e6b93-122">无</span><span class="sxs-lookup"><span data-stu-id="e6b93-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6b93-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e6b93-123">JSON Representation</span></span>
<span data-ttu-id="e6b93-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6b93-124">Here is a JSON representation of the resource.</span></span>
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









