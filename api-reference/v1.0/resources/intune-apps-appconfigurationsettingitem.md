---
title: appConfigurationSettingItem 资源类型
description: 包含应用配置设置项的属性。
author: tfitzmac
ms.openlocfilehash: b75579e56602ad5359bc32d52312931342b42a6b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353576"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="defb4-103">appConfigurationSettingItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="defb4-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="defb4-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="defb4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="defb4-105">包含应用配置设置项的属性。</span><span class="sxs-lookup"><span data-stu-id="defb4-105">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="defb4-106">属性</span><span class="sxs-lookup"><span data-stu-id="defb4-106">Properties</span></span>
|<span data-ttu-id="defb4-107">属性</span><span class="sxs-lookup"><span data-stu-id="defb4-107">Property</span></span>|<span data-ttu-id="defb4-108">类型</span><span class="sxs-lookup"><span data-stu-id="defb4-108">Type</span></span>|<span data-ttu-id="defb4-109">说明</span><span class="sxs-lookup"><span data-stu-id="defb4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="defb4-110">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="defb4-110">appConfigKey</span></span>|<span data-ttu-id="defb4-111">String</span><span class="sxs-lookup"><span data-stu-id="defb4-111">String</span></span>|<span data-ttu-id="defb4-112">应用配置密钥。</span><span class="sxs-lookup"><span data-stu-id="defb4-112">app configuration key.</span></span>|
|<span data-ttu-id="defb4-113">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="defb4-113">appConfigKeyType</span></span>|[<span data-ttu-id="defb4-114">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="defb4-114">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="defb4-115">应用配置密钥类型。</span><span class="sxs-lookup"><span data-stu-id="defb4-115">app configuration key type.</span></span> <span data-ttu-id="defb4-116">可取值为：`stringType`、`integerType`、`realType`、`booleanType`、`tokenType`。</span><span class="sxs-lookup"><span data-stu-id="defb4-116">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="defb4-117">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="defb4-117">appConfigKeyValue</span></span>|<span data-ttu-id="defb4-118">String</span><span class="sxs-lookup"><span data-stu-id="defb4-118">String</span></span>|<span data-ttu-id="defb4-119">应用配置密钥值。</span><span class="sxs-lookup"><span data-stu-id="defb4-119">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="defb4-120">关系</span><span class="sxs-lookup"><span data-stu-id="defb4-120">Relationships</span></span>
<span data-ttu-id="defb4-121">无</span><span class="sxs-lookup"><span data-stu-id="defb4-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="defb4-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="defb4-122">JSON Representation</span></span>
<span data-ttu-id="defb4-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="defb4-123">Here is a JSON representation of the resource.</span></span>
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



