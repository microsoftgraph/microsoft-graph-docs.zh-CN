---
title: windowsInformationProtectionDataRecoveryCertificate 资源类型
description: Windows 信息保护 DataRecoveryCertificate
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 272a1e5f7bf1df1c9e16b2239caeee94cc81f12d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453993"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="0b6ad-103">windowsInformationProtectionDataRecoveryCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="0b6ad-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="0b6ad-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0b6ad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b6ad-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0b6ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b6ad-106">Windows 信息保护 DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="0b6ad-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="0b6ad-107">属性</span><span class="sxs-lookup"><span data-stu-id="0b6ad-107">Properties</span></span>
|<span data-ttu-id="0b6ad-108">属性</span><span class="sxs-lookup"><span data-stu-id="0b6ad-108">Property</span></span>|<span data-ttu-id="0b6ad-109">类型</span><span class="sxs-lookup"><span data-stu-id="0b6ad-109">Type</span></span>|<span data-ttu-id="0b6ad-110">描述</span><span class="sxs-lookup"><span data-stu-id="0b6ad-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b6ad-111">SubjectName</span><span class="sxs-lookup"><span data-stu-id="0b6ad-111">subjectName</span></span>|<span data-ttu-id="0b6ad-112">String</span><span class="sxs-lookup"><span data-stu-id="0b6ad-112">String</span></span>|<span data-ttu-id="0b6ad-113">数据恢复证书主题名称</span><span class="sxs-lookup"><span data-stu-id="0b6ad-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="0b6ad-114">description</span><span class="sxs-lookup"><span data-stu-id="0b6ad-114">description</span></span>|<span data-ttu-id="0b6ad-115">字符串</span><span class="sxs-lookup"><span data-stu-id="0b6ad-115">String</span></span>|<span data-ttu-id="0b6ad-116">数据恢复证书说明</span><span class="sxs-lookup"><span data-stu-id="0b6ad-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="0b6ad-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0b6ad-117">expirationDateTime</span></span>|<span data-ttu-id="0b6ad-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b6ad-118">DateTimeOffset</span></span>|<span data-ttu-id="0b6ad-119">数据恢复证书过期日期/时间</span><span class="sxs-lookup"><span data-stu-id="0b6ad-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="0b6ad-120">证书</span><span class="sxs-lookup"><span data-stu-id="0b6ad-120">certificate</span></span>|<span data-ttu-id="0b6ad-121">Binary</span><span class="sxs-lookup"><span data-stu-id="0b6ad-121">Binary</span></span>|<span data-ttu-id="0b6ad-122">数据恢复证书</span><span class="sxs-lookup"><span data-stu-id="0b6ad-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b6ad-123">关系</span><span class="sxs-lookup"><span data-stu-id="0b6ad-123">Relationships</span></span>
<span data-ttu-id="0b6ad-124">无</span><span class="sxs-lookup"><span data-stu-id="0b6ad-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b6ad-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b6ad-125">JSON Representation</span></span>
<span data-ttu-id="0b6ad-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b6ad-126">Here is a JSON representation of the resource.</span></span>
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





