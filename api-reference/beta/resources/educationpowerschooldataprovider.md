---
title: educationPowerSchoolDataProvider 资源
description: 用于 PowerSchool 用作输入源时设置学校数据同步配置文件。
ms.openlocfilehash: 4c58d3b8baf1569aaeff68375b2dd3643db8b063
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046868"
---
# <a name="educationpowerschooldataprovider-resource"></a><span data-ttu-id="f9ae8-103">educationPowerSchoolDataProvider 资源</span><span class="sxs-lookup"><span data-stu-id="f9ae8-103">educationPowerSchoolDataProvider resource</span></span>

> <span data-ttu-id="f9ae8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f9ae8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9ae8-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f9ae8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f9ae8-106">用于[PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/)用作输入源时设置学校数据同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="f9ae8-106">Used to set up the school data synchronization profile when [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) is used as the input source.</span></span>

<span data-ttu-id="f9ae8-107">派生自[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="f9ae8-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f9ae8-108">属性</span><span class="sxs-lookup"><span data-stu-id="f9ae8-108">Properties</span></span>

| <span data-ttu-id="f9ae8-109">属性</span><span class="sxs-lookup"><span data-stu-id="f9ae8-109">Property</span></span> | <span data-ttu-id="f9ae8-110">类型</span><span class="sxs-lookup"><span data-stu-id="f9ae8-110">Type</span></span> | <span data-ttu-id="f9ae8-111">说明</span><span class="sxs-lookup"><span data-stu-id="f9ae8-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="f9ae8-112">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="f9ae8-112">**connectionUrl**</span></span> | <span data-ttu-id="f9ae8-113">字符串</span><span class="sxs-lookup"><span data-stu-id="f9ae8-113">String</span></span> | <span data-ttu-id="f9ae8-114">连接到 PowerSchool 实例 URL。</span><span class="sxs-lookup"><span data-stu-id="f9ae8-114">The connection URL to the PowerSchool instance.</span></span> |
| <span data-ttu-id="f9ae8-115">**clientId**</span><span class="sxs-lookup"><span data-stu-id="f9ae8-115">**clientId**</span></span> | <span data-ttu-id="f9ae8-116">字符串</span><span class="sxs-lookup"><span data-stu-id="f9ae8-116">String</span></span> |  <span data-ttu-id="f9ae8-117">用于连接到 PowerSchool 客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="f9ae8-117">The client ID used to connect to PowerSchool.</span></span> |
| <span data-ttu-id="f9ae8-118">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="f9ae8-118">**clientSecret**</span></span> | <span data-ttu-id="f9ae8-119">字符串</span><span class="sxs-lookup"><span data-stu-id="f9ae8-119">String</span></span> |  <span data-ttu-id="f9ae8-120">客户端机密进行身份验证与 PowerSchool 实例的连接。</span><span class="sxs-lookup"><span data-stu-id="f9ae8-120">The client secret to authenticate the connection to the PowerSchool instance.</span></span> |
| <span data-ttu-id="f9ae8-121">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="f9ae8-121">**schoolsIds**</span></span> | <span data-ttu-id="f9ae8-122">String 集合</span><span class="sxs-lookup"><span data-stu-id="f9ae8-122">String collection</span></span> |  <span data-ttu-id="f9ae8-123">学校同步的列表。</span><span class="sxs-lookup"><span data-stu-id="f9ae8-123">The list of schools to sync.</span></span> |
| <span data-ttu-id="f9ae8-124">**schoolYear**</span><span class="sxs-lookup"><span data-stu-id="f9ae8-124">**schoolYear**</span></span> | <span data-ttu-id="f9ae8-125">字符串</span><span class="sxs-lookup"><span data-stu-id="f9ae8-125">String</span></span> |  <span data-ttu-id="f9ae8-126">要同步的学校年份。</span><span class="sxs-lookup"><span data-stu-id="f9ae8-126">The school year to sync.</span></span> |
| <span data-ttu-id="f9ae8-127">**allowTeachersInMultipleSchools**</span><span class="sxs-lookup"><span data-stu-id="f9ae8-127">**allowTeachersInMultipleSchools**</span></span> | <span data-ttu-id="f9ae8-128">布尔</span><span class="sxs-lookup"><span data-stu-id="f9ae8-128">Boolean</span></span> |  <span data-ttu-id="f9ae8-129">指示源是否有多个标识符是单个学生或教师。</span><span class="sxs-lookup"><span data-stu-id="f9ae8-129">Indicates whether the source has multiple identifiers for a single student or teacher.</span></span> |
| <span data-ttu-id="f9ae8-130">**自定义项**</span><span class="sxs-lookup"><span data-stu-id="f9ae8-130">**customizations**</span></span> | [<span data-ttu-id="f9ae8-131">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="f9ae8-131">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="f9ae8-132">可选自定义要应用于同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="f9ae8-132">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f9ae8-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f9ae8-133">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationPowerSchoolDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationPowerSchoolDataProvider",
    "connectionUrl": "String",
    "clientId": "String",
    "clientSecret": "String",
    "schoolsids": ["String"],
    "schoolYear": "String",
    "allowTeachersInMultipleSchools": "Boolean",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
