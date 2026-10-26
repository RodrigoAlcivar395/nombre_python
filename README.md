class Empleado:
    nombre = "Issac"
    puesto = "Programador"
    sueldo_por_dia = 300
    dias_trabajados = 15
    iva = 0.16

    def sueldo_bruto(self):
        bruto = self.sueldo_por_dia * self.dias_trabajados
        return bruto

    def sueldo_neto(self):
        bruto = self.sueldo_por_dia * self.dias_trabajados
        neto = bruto - (bruto * self.iva)
        return neto

empleado_1 = Empleado()

print("Nombre del empleado:", empleado_1.nombre)
print("Puesto:", empleado_1.puesto)
print("Sueldo bruto (15 días): $", empleado_1.sueldo_bruto())
print("Sueldo neto con IVA 16% descontado: $", empleado_1.sueldo_neto())
