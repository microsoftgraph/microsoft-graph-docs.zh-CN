---
title: appConfigurationSettingItem 资源类型
description: 包含应用配置设置项的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 11ef3a964d166301c04c49730ac084b68e700b7c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503588"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="9945d-103">appConfigurationSettingItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="9945d-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="9945d-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9945d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9945d-105">包含应用配置设置项的属性。</span><span class="sxs-lookup"><span data-stu-id="9945d-105">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="9945d-106">属性</span><span class="sxs-lookup"><span data-stu-id="9945d-106">Properties</span></span>
|<span data-ttu-id="9945d-107">属性</span><span class="sxs-lookup"><span data-stu-id="9945d-107">Property</span></span>|<span data-ttu-id="9945d-108">类型</span><span class="sxs-lookup"><span data-stu-id="9945d-108">Type</span></span>|<span data-ttu-id="9945d-109">说明</span><span class="sxs-lookup"><span data-stu-id="9945d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9945d-110">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="9945d-110">appConfigKey</span></span>|<span data-ttu-id="9945d-111">字符串</span><span class="sxs-lookup"><span data-stu-id="9945d-111">String</span></span>|<span data-ttu-id="9945d-112">应用配置密钥。</span><span class="sxs-lookup"><span data-stu-id="9945d-112">app configuration key.</span></span>|
|<span data-ttu-id="9945d-113">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="9945d-113">appConfigKeyType</span></span>|[<span data-ttu-id="9945d-114">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="9945d-114">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="9945d-115">应用配置密钥类型。</span><span class="sxs-lookup"><span data-stu-id="9945d-115">app configuration key type.</span></span> <span data-ttu-id="9945d-116">可取值为：`stringType`、`integerType`、`realType`、`booleanType`、`tokenType`。</span><span class="sxs-lookup"><span data-stu-id="9945d-116">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="9945d-117">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="9945d-117">appConfigKeyValue</span></span>|<span data-ttu-id="9945d-118">String</span><span class="sxs-lookup"><span data-stu-id="9945d-118">String</span></span>|<span data-ttu-id="9945d-119">应用配置密钥值。</span><span class="sxs-lookup"><span data-stu-id="9945d-119">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9945d-120">关系</span><span class="sxs-lookup"><span data-stu-id="9945d-120">Relationships</span></span>
<span data-ttu-id="9945d-121">无</span><span class="sxs-lookup"><span data-stu-id="9945d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9945d-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9945d-122">JSON Representation</span></span>
<span data-ttu-id="9945d-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9945d-123">Here is a JSON representation of the resource.</span></span>
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



