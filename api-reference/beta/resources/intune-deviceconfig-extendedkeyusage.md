---
title: extendedKeyUsage 资源类型
description: 自定义扩展密钥用法定义
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cd89a46c2739f80a0a5c661884fb5e72c6e17522
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556149"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="cd213-103">extendedKeyUsage 资源类型</span><span class="sxs-lookup"><span data-stu-id="cd213-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="cd213-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cd213-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd213-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cd213-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd213-106">自定义扩展密钥用法定义</span><span class="sxs-lookup"><span data-stu-id="cd213-106">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="cd213-107">属性</span><span class="sxs-lookup"><span data-stu-id="cd213-107">Properties</span></span>
|<span data-ttu-id="cd213-108">属性</span><span class="sxs-lookup"><span data-stu-id="cd213-108">Property</span></span>|<span data-ttu-id="cd213-109">类型</span><span class="sxs-lookup"><span data-stu-id="cd213-109">Type</span></span>|<span data-ttu-id="cd213-110">说明</span><span class="sxs-lookup"><span data-stu-id="cd213-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd213-111">name</span><span class="sxs-lookup"><span data-stu-id="cd213-111">name</span></span>|<span data-ttu-id="cd213-112">String</span><span class="sxs-lookup"><span data-stu-id="cd213-112">String</span></span>|<span data-ttu-id="cd213-113">扩展密钥用法名称</span><span class="sxs-lookup"><span data-stu-id="cd213-113">Extended Key Usage Name</span></span>|
|<span data-ttu-id="cd213-114">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="cd213-114">objectIdentifier</span></span>|<span data-ttu-id="cd213-115">String</span><span class="sxs-lookup"><span data-stu-id="cd213-115">String</span></span>|<span data-ttu-id="cd213-116">扩展密钥用法对象标识符</span><span class="sxs-lookup"><span data-stu-id="cd213-116">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd213-117">关系</span><span class="sxs-lookup"><span data-stu-id="cd213-117">Relationships</span></span>
<span data-ttu-id="cd213-118">无</span><span class="sxs-lookup"><span data-stu-id="cd213-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd213-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cd213-119">JSON Representation</span></span>
<span data-ttu-id="cd213-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd213-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.extendedKeyUsage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extendedKeyUsage",
  "name": "String",
  "objectIdentifier": "String"
}
```





