---
title: appConfigurationSettingItem 资源类型
description: 包含应用配置设置项的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: af738e6c5f558b7460c8cbd7c5e02abae3dbb922
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756083"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="127a0-103">appConfigurationSettingItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="127a0-103">appConfigurationSettingItem resource type</span></span>

<span data-ttu-id="127a0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="127a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="127a0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="127a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="127a0-106">包含应用配置设置项的属性。</span><span class="sxs-lookup"><span data-stu-id="127a0-106">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="127a0-107">属性</span><span class="sxs-lookup"><span data-stu-id="127a0-107">Properties</span></span>
|<span data-ttu-id="127a0-108">属性</span><span class="sxs-lookup"><span data-stu-id="127a0-108">Property</span></span>|<span data-ttu-id="127a0-109">类型</span><span class="sxs-lookup"><span data-stu-id="127a0-109">Type</span></span>|<span data-ttu-id="127a0-110">Description</span><span class="sxs-lookup"><span data-stu-id="127a0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="127a0-111">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="127a0-111">appConfigKey</span></span>|<span data-ttu-id="127a0-112">String</span><span class="sxs-lookup"><span data-stu-id="127a0-112">String</span></span>|<span data-ttu-id="127a0-113">应用配置密钥。</span><span class="sxs-lookup"><span data-stu-id="127a0-113">app configuration key.</span></span>|
|<span data-ttu-id="127a0-114">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="127a0-114">appConfigKeyType</span></span>|[<span data-ttu-id="127a0-115">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="127a0-115">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="127a0-116">应用配置密钥类型。</span><span class="sxs-lookup"><span data-stu-id="127a0-116">app configuration key type.</span></span> <span data-ttu-id="127a0-117">可取值为：`stringType`、`integerType`、`realType`、`booleanType`、`tokenType`。</span><span class="sxs-lookup"><span data-stu-id="127a0-117">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="127a0-118">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="127a0-118">appConfigKeyValue</span></span>|<span data-ttu-id="127a0-119">String</span><span class="sxs-lookup"><span data-stu-id="127a0-119">String</span></span>|<span data-ttu-id="127a0-120">应用配置密钥值。</span><span class="sxs-lookup"><span data-stu-id="127a0-120">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="127a0-121">关系</span><span class="sxs-lookup"><span data-stu-id="127a0-121">Relationships</span></span>
<span data-ttu-id="127a0-122">无</span><span class="sxs-lookup"><span data-stu-id="127a0-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="127a0-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="127a0-123">JSON Representation</span></span>
<span data-ttu-id="127a0-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="127a0-124">Here is a JSON representation of the resource.</span></span>
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




