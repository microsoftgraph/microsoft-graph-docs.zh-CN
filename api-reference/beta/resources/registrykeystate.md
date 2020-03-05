---
title: registryKeyState 资源类型
description: 包含有关与警报相关的注册表项更改的信息，以及更改了注册表项的过程。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 8f8f5aa0458666dfc10c4a3066534ea66821fb3a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521192"
---
# <a name="registrykeystate-resource-type"></a><span data-ttu-id="38eda-103">registryKeyState 资源类型</span><span class="sxs-lookup"><span data-stu-id="38eda-103">registryKeyState resource type</span></span>

<span data-ttu-id="38eda-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="38eda-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="38eda-105">包含有关与警报相关的注册表项更改的信息，以及更改了注册表项的过程。</span><span class="sxs-lookup"><span data-stu-id="38eda-105">Contains information about registry key changes related to the alert, and the process that changed the registry keys.</span></span>

## <a name="properties"></a><span data-ttu-id="38eda-106">属性</span><span class="sxs-lookup"><span data-stu-id="38eda-106">Properties</span></span>

| <span data-ttu-id="38eda-107">属性</span><span class="sxs-lookup"><span data-stu-id="38eda-107">Property</span></span>     | <span data-ttu-id="38eda-108">类型</span><span class="sxs-lookup"><span data-stu-id="38eda-108">Type</span></span>        | <span data-ttu-id="38eda-109">说明</span><span class="sxs-lookup"><span data-stu-id="38eda-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="38eda-110">配置单元</span><span class="sxs-lookup"><span data-stu-id="38eda-110">hive</span></span>|<span data-ttu-id="38eda-111">registryHive</span><span class="sxs-lookup"><span data-stu-id="38eda-111">registryHive</span></span>|<span data-ttu-id="38eda-112">[Windows 注册表配置单元](/windows/desktop/sysinfo/registry-hives)：</span><span class="sxs-lookup"><span data-stu-id="38eda-112">A [Windows registry hive](/windows/desktop/sysinfo/registry-hives) :</span></span> <ul><li><span data-ttu-id="38eda-113">HKEY_CURRENT_CONFIG</span><span class="sxs-lookup"><span data-stu-id="38eda-113">HKEY_CURRENT_CONFIG</span></span></li> <li><span data-ttu-id="38eda-114">HKEY_CURRENT_USER</span><span class="sxs-lookup"><span data-stu-id="38eda-114">HKEY_CURRENT_USER</span></span></li> <li><span data-ttu-id="38eda-115">HKEY_LOCAL_MACHINE \SAM</span><span class="sxs-lookup"><span data-stu-id="38eda-115">HKEY_LOCAL_MACHINE\SAM</span></span></li> <li><span data-ttu-id="38eda-116">HKEY_LOCAL_MACHINE \Security</span><span class="sxs-lookup"><span data-stu-id="38eda-116">HKEY_LOCAL_MACHINE\Security</span></span></li> <li><span data-ttu-id="38eda-117">HKEY_LOCAL_MACHINE \Software</span><span class="sxs-lookup"><span data-stu-id="38eda-117">HKEY_LOCAL_MACHINE\Software</span></span></li> <li><span data-ttu-id="38eda-118">HKEY_LOCAL_MACHINE \System</span><span class="sxs-lookup"><span data-stu-id="38eda-118">HKEY_LOCAL_MACHINE\System</span></span></li> <li><span data-ttu-id="38eda-119">HKEY_USERS\\。设置.</span><span class="sxs-lookup"><span data-stu-id="38eda-119">HKEY_USERS\\.Default.</span></span></li></ul> <span data-ttu-id="38eda-120">可取值为：`unknown`、`currentConfig`、`currentUser`、`localMachineSam`、`localMachineSecurity`、`localMachineSoftware`、`localMachineSystem`、`usersDefault`。</span><span class="sxs-lookup"><span data-stu-id="38eda-120">Possible values are: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSecurity`, `localMachineSoftware`, `localMachineSystem`, `usersDefault`.</span></span>|
|<span data-ttu-id="38eda-121">注册表项</span><span class="sxs-lookup"><span data-stu-id="38eda-121">key</span></span>|<span data-ttu-id="38eda-122">String</span><span class="sxs-lookup"><span data-stu-id="38eda-122">String</span></span>|<span data-ttu-id="38eda-123">当前（如已更改）的注册表项（不包括配置单元）。</span><span class="sxs-lookup"><span data-stu-id="38eda-123">Current (i.e. changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="38eda-124">oldKey</span><span class="sxs-lookup"><span data-stu-id="38eda-124">oldKey</span></span>|<span data-ttu-id="38eda-125">String</span><span class="sxs-lookup"><span data-stu-id="38eda-125">String</span></span>|<span data-ttu-id="38eda-126">上一个（即 "更改前"）注册表项（不包括 HIVE）。</span><span class="sxs-lookup"><span data-stu-id="38eda-126">Previous (i.e. before changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="38eda-127">oldValueData</span><span class="sxs-lookup"><span data-stu-id="38eda-127">oldValueData</span></span>|<span data-ttu-id="38eda-128">String</span><span class="sxs-lookup"><span data-stu-id="38eda-128">String</span></span>|<span data-ttu-id="38eda-129">以前的（即更改之前）注册表项值数据（内容）。</span><span class="sxs-lookup"><span data-stu-id="38eda-129">Previous (i.e. before changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="38eda-130">oldValueName</span><span class="sxs-lookup"><span data-stu-id="38eda-130">oldValueName</span></span>|<span data-ttu-id="38eda-131">String</span><span class="sxs-lookup"><span data-stu-id="38eda-131">String</span></span>|<span data-ttu-id="38eda-132">以前的注册表项值名称（即 "更改前"）。</span><span class="sxs-lookup"><span data-stu-id="38eda-132">Previous (i.e. before changed) registry key value name.</span></span>|
|<span data-ttu-id="38eda-133">操作</span><span class="sxs-lookup"><span data-stu-id="38eda-133">operation</span></span>|<span data-ttu-id="38eda-134">registryOperation</span><span class="sxs-lookup"><span data-stu-id="38eda-134">registryOperation</span></span>|<span data-ttu-id="38eda-135">更改注册表项名称和/或值的操作。</span><span class="sxs-lookup"><span data-stu-id="38eda-135">Operation that changed the registry key name and/or value.</span></span> <span data-ttu-id="38eda-136">可取值为：`unknown`、`create`、`modify`、`delete`。</span><span class="sxs-lookup"><span data-stu-id="38eda-136">Possible values are: `unknown`, `create`, `modify`, `delete`.</span></span>|
|<span data-ttu-id="38eda-137">processId</span><span class="sxs-lookup"><span data-stu-id="38eda-137">processId</span></span>|<span data-ttu-id="38eda-138">Int32</span><span class="sxs-lookup"><span data-stu-id="38eda-138">Int32</span></span>|<span data-ttu-id="38eda-139">修改注册表项的进程的进程 ID （PID）（进程详细信息将显示在警报的 "进程" 集合中）。</span><span class="sxs-lookup"><span data-stu-id="38eda-139">Process ID (PID) of the process that modified the registry key (process details will appear in the alert 'processes' collection).</span></span>|
|<span data-ttu-id="38eda-140">valueData</span><span class="sxs-lookup"><span data-stu-id="38eda-140">valueData</span></span>|<span data-ttu-id="38eda-141">String</span><span class="sxs-lookup"><span data-stu-id="38eda-141">String</span></span>|<span data-ttu-id="38eda-142">当前（如已更改）的注册表项值数据（内容）。</span><span class="sxs-lookup"><span data-stu-id="38eda-142">Current (i.e. changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="38eda-143">等值</span><span class="sxs-lookup"><span data-stu-id="38eda-143">valueName</span></span>|<span data-ttu-id="38eda-144">String</span><span class="sxs-lookup"><span data-stu-id="38eda-144">String</span></span>|<span data-ttu-id="38eda-145">当前（如已更改）的注册表项值名称</span><span class="sxs-lookup"><span data-stu-id="38eda-145">Current (i.e. changed) registry key value name</span></span>|
|<span data-ttu-id="38eda-146">valueType</span><span class="sxs-lookup"><span data-stu-id="38eda-146">valueType</span></span>|<span data-ttu-id="38eda-147">registryValueType</span><span class="sxs-lookup"><span data-stu-id="38eda-147">registryValueType</span></span>|[<span data-ttu-id="38eda-148">注册表项值类型</span><span class="sxs-lookup"><span data-stu-id="38eda-148">Registry key value type</span></span>](/windows/desktop/sysinfo/registry-value-types) <ul><li><span data-ttu-id="38eda-149">REG_BINARY</span><span class="sxs-lookup"><span data-stu-id="38eda-149">REG_BINARY</span></span></li> <li><span data-ttu-id="38eda-150">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="38eda-150">REG_DWORD</span></span></li> <li><span data-ttu-id="38eda-151">REG_DWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="38eda-151">REG_DWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="38eda-152">REG_DWORD_BIG_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="38eda-152">REG_DWORD_BIG_ENDIAN</span></span></li><li><span data-ttu-id="38eda-153">REG_EXPAND_SZ</span><span class="sxs-lookup"><span data-stu-id="38eda-153">REG_EXPAND_SZ</span></span></li> <li><span data-ttu-id="38eda-154">REG_LINK</span><span class="sxs-lookup"><span data-stu-id="38eda-154">REG_LINK</span></span></li> <li><span data-ttu-id="38eda-155">REG_MULTI_SZ</span><span class="sxs-lookup"><span data-stu-id="38eda-155">REG_MULTI_SZ</span></span></li> <li><span data-ttu-id="38eda-156">REG_NONE</span><span class="sxs-lookup"><span data-stu-id="38eda-156">REG_NONE</span></span></li> <li><span data-ttu-id="38eda-157">REG_QWORD</span><span class="sxs-lookup"><span data-stu-id="38eda-157">REG_QWORD</span></span></li> <li><span data-ttu-id="38eda-158">REG_QWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="38eda-158">REG_QWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="38eda-159">REG_SZ</span><span class="sxs-lookup"><span data-stu-id="38eda-159">REG_SZ</span></span></li></ul> <span data-ttu-id="38eda-160">可取值为：`unknown`、`binary`、`dword`、`dwordLittleEndian`、`dwordBigEndian`、`expandSz`、`link`、`multiSz`、`none`、`qword`、`qwordlittleEndian`、`sz`。</span><span class="sxs-lookup"><span data-stu-id="38eda-160">Possible values are: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="38eda-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="38eda-161">JSON representation</span></span>

<span data-ttu-id="38eda-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38eda-162">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.registryKeyState"
}-->

```json
{
  "hive": "@odata.type: microsoft.graph.registryHive",
  "key": "String",
  "oldKey": "String",
  "oldValueData": "String",
  "oldValueName": "String",
  "operation": "@odata.type: microsoft.graph.registryOperation",
  "processId": 1024,
  "valueData": "String",
  "valueName": "String",
  "valueType": "@odata.type: microsoft.graph.registryValueType"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "registryKeyState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
