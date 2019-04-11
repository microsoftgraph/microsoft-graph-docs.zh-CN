---
title: windowsInformationProtectionDataRecoveryCertificate 资源类型
description: Windows 信息保护 DataRecoveryCertificate
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 272a1e5f7bf1df1c9e16b2239caeee94cc81f12d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790632"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="81a5f-103">windowsInformationProtectionDataRecoveryCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="81a5f-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="81a5f-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="81a5f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81a5f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="81a5f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81a5f-106">Windows 信息保护 DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="81a5f-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="81a5f-107">属性</span><span class="sxs-lookup"><span data-stu-id="81a5f-107">Properties</span></span>
|<span data-ttu-id="81a5f-108">属性</span><span class="sxs-lookup"><span data-stu-id="81a5f-108">Property</span></span>|<span data-ttu-id="81a5f-109">类型</span><span class="sxs-lookup"><span data-stu-id="81a5f-109">Type</span></span>|<span data-ttu-id="81a5f-110">说明</span><span class="sxs-lookup"><span data-stu-id="81a5f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81a5f-111">SubjectName</span><span class="sxs-lookup"><span data-stu-id="81a5f-111">subjectName</span></span>|<span data-ttu-id="81a5f-112">String</span><span class="sxs-lookup"><span data-stu-id="81a5f-112">String</span></span>|<span data-ttu-id="81a5f-113">数据恢复证书主题名称</span><span class="sxs-lookup"><span data-stu-id="81a5f-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="81a5f-114">description</span><span class="sxs-lookup"><span data-stu-id="81a5f-114">description</span></span>|<span data-ttu-id="81a5f-115">String</span><span class="sxs-lookup"><span data-stu-id="81a5f-115">String</span></span>|<span data-ttu-id="81a5f-116">数据恢复证书说明</span><span class="sxs-lookup"><span data-stu-id="81a5f-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="81a5f-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="81a5f-117">expirationDateTime</span></span>|<span data-ttu-id="81a5f-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81a5f-118">DateTimeOffset</span></span>|<span data-ttu-id="81a5f-119">数据恢复证书过期日期/时间</span><span class="sxs-lookup"><span data-stu-id="81a5f-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="81a5f-120">证书</span><span class="sxs-lookup"><span data-stu-id="81a5f-120">certificate</span></span>|<span data-ttu-id="81a5f-121">Binary</span><span class="sxs-lookup"><span data-stu-id="81a5f-121">Binary</span></span>|<span data-ttu-id="81a5f-122">数据恢复证书</span><span class="sxs-lookup"><span data-stu-id="81a5f-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="81a5f-123">关系</span><span class="sxs-lookup"><span data-stu-id="81a5f-123">Relationships</span></span>
<span data-ttu-id="81a5f-124">无</span><span class="sxs-lookup"><span data-stu-id="81a5f-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81a5f-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81a5f-125">JSON Representation</span></span>
<span data-ttu-id="81a5f-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81a5f-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```





